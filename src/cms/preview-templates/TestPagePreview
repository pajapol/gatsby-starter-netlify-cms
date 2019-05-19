import React from 'react'
import PropTypes from 'prop-types'
import { TestPageTemplate } from '../../templates/test-page'

const TestPagePreview = ({ entry, getAsset }) => {
  const data = entry.getIn(['data']).toJS()

  if (data) {
    return (
      <TestPageTemplate
        image={data.image}
        title={data.title}
        heading={data.heading}
      
      />
    )
  } else {
    return <div>Loading...</div>
  }
}

TestPagePreview.propTypes = {
  entry: PropTypes.shape({
    getIn: PropTypes.func,
  }),
  getAsset: PropTypes.func,
}

export default TestPagePreview
